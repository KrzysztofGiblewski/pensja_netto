unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, FileUtil, Forms, Controls, Graphics, Dialogs, Spin,
  StdCtrls;

type

  { TForm1 }

  TForm1 = class(TForm)
    Button1: TButton;
    Button2: TButton;
    Button3: TButton;
    FloatSpinEdit1: TFloatSpinEdit;
    FloatSpinEdit10: TFloatSpinEdit;
    FloatSpinEdit11: TFloatSpinEdit;
    FloatSpinEdit12: TFloatSpinEdit;
    FloatSpinEdit2: TFloatSpinEdit;
    FloatSpinEdit3: TFloatSpinEdit;
    FloatSpinEdit4: TFloatSpinEdit;
    FloatSpinEdit5: TFloatSpinEdit;
    FloatSpinEdit6: TFloatSpinEdit;
    FloatSpinEdit7: TFloatSpinEdit;
    FloatSpinEdit8: TFloatSpinEdit;
    FloatSpinEdit9: TFloatSpinEdit;
    Label1: TLabel;
    Label10: TLabel;
    Label11: TLabel;
    Label12: TLabel;
    Label13: TLabel;
    Label14: TLabel;
    Label15: TLabel;
    Label16: TLabel;
    Label17: TLabel;
    Label18: TLabel;
    Label19: TLabel;
    Label2: TLabel;
    Label20: TLabel;
    Label21: TLabel;
    Label22: TLabel;
    Label23: TLabel;
    Label24: TLabel;
    Label25: TLabel;
    Label3: TLabel;
    Label4: TLabel;
    Label5: TLabel;
    Label6: TLabel;
    Label7: TLabel;
    Label8: TLabel;
    Label9: TLabel;
    SpinEdit2: TSpinEdit;
    SpinEdit3: TSpinEdit;
    SpinEdit5: TSpinEdit;
    procedure Button1Click(Sender: TObject);
    procedure Button2Click(Sender: TObject);
    procedure Button3Click(Sender: TObject);
    procedure FormCreate(Sender: TObject);
  private
    { private declarations }
  public
    { public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.lfm}

{ TForm1 }

procedure TForm1.Button1Click(Sender: TObject);
begin
  application.Terminate;
end;

procedure TForm1.Button2Click(Sender: TObject);
var

  stawka, godzin, gnocki,
  dodate, premia, potrac,
  pensjaBrutto,pensjaNetto,
  srg, nrg ,xx , yy, zz, aaa,
  podatek18, skemeryt,skchoro ,skrent ,ubzdrow ,
  kosztuzys , kwotawolna, skubezpie
  :extended;

begin
  stawka:=floatspinedit1.Value;
  godzin:=spinedit2.Value;
  gnocki:=spinedit3.Value;
  dodate:=floatspinedit2.Value;
  premia:=spinedit5.Value;
  podatek18:=floatspinedit3.Value ;
  skemeryt:=floatspinedit4.Value ;
  skchoro:=floatspinedit5.Value ;
  skrent:=floatspinedit6.Value ;
  ubzdrow:=floatspinedit7.Value ;
  kosztuzys:=floatspinedit8.Value ;
  kwotawolna:=floatspinedit9.Value ;
  skubezpie:=floatspinedit10.Value ;

     srg:=stawka*godzin;     //brutto bez nocek


      yy:=srg*premia*0.01;   //obliczam premie
           label7.Caption:=floattostr(yy)+' premi brutto';

   nrg:=gnocki*dodate;     //licze dodatek za nocki

       label10.Caption:='z czego '+floattostr(nrg)+' dodatku za nocki';

       aaa:=srg+nrg+yy;

     label11.Caption:=floattostr(srg)+'stawka razy ilosc godzin+'+floattostr(nrg)+
                                              ' dodatku za nocki+'+floattostr(yy)+
                                              'premia = '+floattostr(aaa)+' brutto'; //stawka razy godziny plus nocki





     xx:=yy+srg;     //suma yy czyli premia brutto za godziny i dodatek nocny
     zz:=xx*0.3; // robie 30 procent potracen
     label8.Caption:=floattostr(zz)+' w przyblizeniu w sumie 30 procent wszystkich potracen';

     pensjaBrutto:=xx;
     pensjaNetto :=(xx)-zz;

     label9.Caption:=floattostr(pensjaNetto)+' Nieco zaokraglona pensja netto (po potraceniu 30 procent)';

end;

procedure TForm1.Button3Click(Sender: TObject);
var

  stawka, godzin, gnocki,
  dodate, premia, potrac, ekstrapremia, ekstrapotracenia,
  pensjaBrutto,pensjaNetto,
  srg, nrg ,xx , yy, zz, xemeryt, xrent, xchorob,
  xpodsklubezzdrow, sumasklspo,  skladzdow7, ostatecznypodatek,
  podstsklubzdr, yubzdro, zaliczkapodatku, podatek,
  podatek18, skemeryt,skchoro ,skrent ,ubzdrow ,
  kosztuzys , kwotawolna, skubezpie
  :extended;

begin
  stawka:=floatspinedit1.Value;
  godzin:=spinedit2.Value;
  gnocki:=spinedit3.Value;
  dodate:=floatspinedit2.Value;
  premia:=spinedit5.Value;
  podatek18:=floatspinedit3.Value ;
  skemeryt:=floatspinedit4.Value ;
  skchoro:=floatspinedit5.Value ;
  skrent:=floatspinedit6.Value ;
  ubzdrow:=floatspinedit7.Value ;
  kosztuzys:=floatspinedit8.Value ;
  kwotawolna:=floatspinedit9.Value ;
  skubezpie:=floatspinedit10.Value ;
  ekstrapremia:=floatspinedit11.Value ;
  ekstrapotracenia:=floatspinedit12.Value;


     srg:=stawka*godzin;     //brutto bez nocek
      nrg:=gnocki*dodate;     //licze dodatek za nocki


     label11.Caption:='liczba godzin razy stawka godzinowa '+floattostr(srg+nrg); //stawka razy godziny plus nocki

     label10.Caption:='z czego '+floattostr(nrg)+' dodatku za nocki';

     yy:=srg*premia*0.01;   //obliczam premie

     label7.Caption:=floattostr(yy)+' premi brutto';

     xx:=yy+srg+nrg+ekstrapremia-ekstrapotracenia;     //suma yy czyli premia brutto za godziny i dodatek nocny i ekstrapremia
     label21.Caption:='podstawa brutto '+floattostr(xx);     //obliczona podstawa brutto

     xemeryt:=xx*skemeryt*0.01;    // skladka emerytalna
     label13.Caption:='skladka emerytalna '+floattostr(xx)+' razy '+floattostr(skemeryt)+'% ='+floattostr(xemeryt);

     xrent:=xx*skrent*0.01;         //skladka rentowa
     label15.Caption:='skladka rentowa '+floattostr(xx)+' razy '+floattostr(skrent)+'% ='+floattostr(xrent);

     xchorob:=xx*skchoro*0.01;          //skladka chorobowa
     label14.Caption:='skladka chorobowa '+floattostr(xx)+' razy '+floattostr(skchoro)+'% ='+floattostr(xchorob);

     sumasklspo:=xemeryt+xrent+xchorob;    //sumuje wszysklie trzy skladki
     label21.Caption:='suma sladek spolecznych= ' +floattostr(sumasklspo);

     podstsklubzdr:=xx-sumasklspo;         //podstawa skladki na ubezpieczenie zdrowotne
     yubzdro:=podstsklubzdr*ubzdrow*0.01;    // obliczam skladke na ubezpieczenie zdrowotne
     label16.Caption:='skladka ubezpieczenia zdrowotnego to podstawa pensji - suma skladek spolecznych '
                                +floattostr(podstsklubzdr)+'razy '+floattostr(ubzdrow)+' % = '+floattostr(yubzdro);

     zaliczkapodatku:= (podstsklubzdr-kosztuzys)*podatek18*0.01;     //podatek to podstawa pomiejszonao skladki i koszt uzyskania razy podatek
     label12.Caption:='zaliczka podatku dochodowego to podstawa pomiejszona o sume skladek spolecznych i koszt uzyskania przychodu '+floattostr(zaliczkapodatku);

     podatek:= zaliczkapodatku-kwotawolna; //podatek to zaliczka minus kwota wolna
     label18.Caption:='kwota wolna od podatku pomniejsza zaliczke podatku i ostatecznie podatek to '+floattostr(podatek);

     skladzdow7:=podstsklubzdr*skubezpie*0.01;  //skladka ubezpieczenie zdrowotne7%
     ostatecznypodatek:=podatek- round(skladzdow7);
     label19.Caption:='skladka na ubezpieczenie zdrowotne '+floattostr(skladzdow7);

      pensjaNetto:=xx- sumasklspo-ostatecznypodatek-yubzdro; //pesja netto
      label20.Caption:='pesja netto wynosi '+floattostr(pensjaNetto);

      label24.Caption:='podstawa brutto '+floattostr(xx);

end;

procedure TForm1.FormCreate(Sender: TObject);
begin

end;

end.

