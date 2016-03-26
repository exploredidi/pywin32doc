# PyCFontDialog

## PyCFontDialog Object

A class which encapsulates an MFC CFontDialog object.  Derived from a[PyCDialog](#pycdialog)object.

#### Methods


  - [DoModal](PyCFontDialog.md#pycfontdialogdomodal)

    Displays a dialog and allows the user to make a selection.&nbsp;

  - [GetCurrentFont](PyCFontDialog.md#pycfontdialoggetcurrentfont)

    Returns a dictionary describing the current font.&nbsp;

  - [GetCharFormat](PyCFontDialog.md#pycfontdialoggetcharformat)

    Returns the font selection in a CHARFORMAT tuple.&nbsp;

  - [GetColor](PyCFontDialog.md#pycfontdialoggetcolor)

    Determines the color of the selected font.&nbsp;

  - [GetFaceName](PyCFontDialog.md#pycfontdialoggetfacename)

    Returns the face name of the selected font.&nbsp;

  - [GetStyleName](PyCFontDialog.md#pycfontdialoggetstylename)

    Returns the style name of the selected font.&nbsp;

  - [GetSize](PyCFontDialog.md#pycfontdialoggetsize)

    Returns he font's size, in tenths of a point.&nbsp;

  - [GetWeight](PyCFontDialog.md#pycfontdialoggetweight)

    Returns the font's weight.&nbsp;

  - [IsStrikeOut](PyCFontDialog.md#pycfontdialogisstrikeout)

    Determines whether the font is displayed with strikeout.&nbsp;

  - [IsUnderline](PyCFontDialog.md#pycfontdialogisunderline)

    Determines whether the font is displayed with underline.&nbsp;

  - [IsBold](PyCFontDialog.md#pycfontdialogisbold)

    Determines whether the font is displayed bold.&nbsp;

  - [IsItalic](PyCFontDialog.md#pycfontdialogisitalic)

    Determines whether the font is displayed with italic.&nbsp;


## [PyCFontDialog](#pycfontdialog).DoModal

int = __DoModal(__ )
Displays a dialog and allows the user to make a selection.

#### MFC References


  - CFontDialog::DoModal

## [PyCFontDialog](#pycfontdialog).GetCharFormat

tuple = __GetCharFormat(__ )
Returns the font selection in a CHARFORMAT tuple.

#### MFC References


  - CFontDialog::GetCharFormat

## [PyCFontDialog](#pycfontdialog).GetColor

int = __GetColor(__ )
Determines the color of the selected font.

#### MFC References


  - CFontDialog::GetColor

## [PyCFontDialog](#pycfontdialog).GetCurrentFont

dict = __GetCurrentFont(__ )
Returns a dictionary describing the current font.

#### MFC References


  - CFontDialog::GetCurrentFont

## [PyCFontDialog](#pycfontdialog).GetFaceName

string = __GetFaceName(__ )
Returns the face name of the selected font.

#### MFC References


  - CFontDialog::GetFaceName

## [PyCFontDialog](#pycfontdialog).GetSize

int = __GetSize(__ )
Returns he font's size, in tenths of a point.

#### MFC References


  - CFontDialog::GetSize

## [PyCFontDialog](#pycfontdialog).GetStyleName

string = __GetStyleName(__ )
Returns the style name of the selected font.

#### MFC References


  - CFontDialog::GetStyleName

## [PyCFontDialog](#pycfontdialog).GetWeight

int = __GetWeight(__ )
Returns the font's weight.

#### MFC References


  - CFontDialog::GetWeight

## [PyCFontDialog](#pycfontdialog).IsBold

int = __IsBold(__ )
Determines whether the font is displayed bold.

#### MFC References


  - CFontDialog::IsBold

## [PyCFontDialog](#pycfontdialog).IsItalic

int = __IsItalic(__ )
Determines whether the font is displayed with italic.

#### MFC References


  - CFontDialog::IsItalic

## [PyCFontDialog](#pycfontdialog).IsStrikeOut

int = __IsStrikeOut(__ )
Determines whether the font is displayed with strikeout.

#### MFC References


  - CFontDialog::IsStrikeOut

## [PyCFontDialog](#pycfontdialog).IsUnderline

int = __IsUnderline(__ )
Determines whether the font is displayed with underline.

#### MFC References


  - CFontDialog::IsUnderline