# PyCButton

## PyCButton Object

A windows button.  Encapsulates an MFC __CButton__ class.  Derived from[PyCControl](#pyccontrol).

#### Methods


  - [CreateWindow](PyCButton.md#pycbuttoncreatewindow)

    Creates the window for a new button object.&nbsp;

  - [GetBitmap](PyCButton.md#pycbuttongetbitmap)

    Retrieves the bitmap associated with the button.&nbsp;

  - [SetBitmap](PyCButton.md#pycbuttonsetbitmap)

    Sets the bitmap of a button.&nbsp;

  - [GetCheck](PyCButton.md#pycbuttongetcheck)

    Retrieves the check state of a radio button or check box.&nbsp;

  - [SetCheck](PyCButton.md#pycbuttonsetcheck)

    Sets the check state of a radio button or check box.&nbsp;

  - [GetState](PyCButton.md#pycbuttongetstate)

    Retrieves the state of a radio button or check box.&nbsp;

  - [SetState](PyCButton.md#pycbuttonsetstate)

    Sets the state of a radio button or check box.&nbsp;

  - [GetButtonStyle](PyCButton.md#pycbuttongetbuttonstyle)

    Retrieves the style of a radio button or check box.&nbsp;

  - [SetButtonStyle](PyCButton.md#pycbuttonsetbuttonstyle)

    Sets the state of a radio button or check box.&nbsp;

## [PyCButton](#pycbutton).CreateWindow

 __CreateWindow( *caption*  *, style*  *, rect*  *, parent*  *, id* __ )
Creates the window for a new button object.

#### Parameters


  -  *caption* : string

    The caption (text) for the button.

  -  *style* : int

    The style for the button.  Use any of the win32con.BS_* constants.

  -  *rect* : (left, top, right, bottom)

    The size and position of the button.

  -  *parent* :[PyCWnd](#pycwnd)

    The parent window of the button.  Usually a[PyCDialog](#pycdialog).

  -  *id* : int

    The buttons control ID.

## [PyCButton](#pycbutton).GetBitmap

int = __GetBitmap(__ )
Get the button's bitmap

## [PyCButton](#pycbutton).GetButtonStyle

int = __GetButtonStyle(__ )
Gets the style of the button.

## [PyCButton](#pycbutton).GetCheck

int = __GetCheck(__ )
Retrieves the check state of a radio button or check box.

## [PyCButton](#pycbutton).GetState

int = __GetState(__ )
Returns the state of the button.

## [PyCButton](#pycbutton).SetBitmap

int = __SetBitmap( *hBitmap* __ )
Set the button's bitmap

#### Parameters


  -  *hBitmap=1* : int

    Handle of the new bitmap

## [PyCButton](#pycbutton).SetButtonStyle

int = __SetButtonStyle( *style*  *, bRedraw* __ )
Sets the style of the button.

#### Parameters


  -  *style* : int

    The new style for the button.

  -  *bRedraw=1* : int

    Should the button be redrawn?

## [PyCButton](#pycbutton).SetCheck

 __SetCheck( *idCheck* __ )
Sets or resets the state of a radio button or check box.

#### Parameters


  -  *idCheck* : int

    The ID of the button.

## [PyCButton](#pycbutton).SetState

int = __SetState( *bHighlight* __ )
Sets the state of the button.

#### Parameters


  -  *bHighlight* : int

    The new state for the button.

#### Comments
Highlighting affects the exterior of a button control. It has no effect on the check state of a radio button or check box.