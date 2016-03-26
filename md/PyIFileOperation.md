# PyIFileOperation

## PyIFileOperation Object

Interface used to build a collection of file system modifications to be 

performed by the shell as a unit.  Serves as a replacement for[shell::SHFileOperation](shell.md#shellshfileoperation).
No changes are actually made until PerformOperations is called.
Progress can be monitored by implementing[PyGFileOperationProgressSink](#pygfileoperationprogresssink).
Requires Vista or later.

#### Methods


  - [Advise](PyIFileOperation.md#pyifileoperationadvise)

    Connects an event sink to receive updates&nbsp;

  - [Unadvise](PyIFileOperation.md#pyifileoperationunadvise)

    Disconnects a progress sink&nbsp;

  - [SetOperationFlags](PyIFileOperation.md#pyifileoperationsetoperationflags)

    Sets option flags&nbsp;

  - [SetProgressMessage](PyIFileOperation.md#pyifileoperationsetprogressmessage)

    Not implemented&nbsp;

  - [SetProgressDialog](PyIFileOperation.md#pyifileoperationsetprogressdialog)

    Provides an interface used to display progress&nbsp;

  - [SetProperties](PyIFileOperation.md#pyifileoperationsetproperties)

    Specifies a set of properties to be changed&nbsp;

  - [SetOwnerWindow](PyIFileOperation.md#pyifileoperationsetownerwindow)

    Sets the parent window for any UI displayed.&nbsp;

  - [ApplyPropertiesToItem](PyIFileOperation.md#pyifileoperationapplypropertiestoitem)

    Specifies the item that will receive property changes&nbsp;

  - [ApplyPropertiesToItems](PyIFileOperation.md#pyifileoperationapplypropertiestoitems)

    Specifies multiple items that will receive property changes&nbsp;

  - [RenameItem](PyIFileOperation.md#pyifileoperationrenameitem)

    Adds a rename to the operation sequence&nbsp;

  - [RenameItems](PyIFileOperation.md#pyifileoperationrenameitems)

    Adds multiple renames to the operation sequence&nbsp;

  - [MoveItem](PyIFileOperation.md#pyifileoperationmoveitem)

    Adds a move operation to the configuration&nbsp;

  - [MoveItems](PyIFileOperation.md#pyifileoperationmoveitems)

    Adds multiple move operations to the configuration&nbsp;

  - [CopyItem](PyIFileOperation.md#pyifileoperationcopyitem)

    Adds a copy operation to the configuration&nbsp;

  - [CopyItems](PyIFileOperation.md#pyifileoperationcopyitems)

    Adds multiple copy operations to the configuration&nbsp;

  - [DeleteItem](PyIFileOperation.md#pyifileoperationdeleteitem)

    Adds a delete operation to the configuration&nbsp;

  - [DeleteItems](PyIFileOperation.md#pyifileoperationdeleteitems)

    Adds multiple delete operations to the configuration&nbsp;

  - [NewItem](PyIFileOperation.md#pyifileoperationnewitem)

    Creates a new file as part of the operation&nbsp;

  - [PerformOperations](PyIFileOperation.md#pyifileoperationperformoperations)

    Effects all configured file system modifications&nbsp;

  - [GetAnyOperationsAborted](PyIFileOperation.md#pyifileoperationgetanyoperationsaborted)

    Determines if any operations were terminated&nbsp;

## [PyIFileOperation](#pyifileoperation).Advise

int = __Advise( *Sink* __ )
Connects an event sink to receive updates

#### Parameters


  -  *Sink* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Interface that receives progress updates

#### Return Value
Returns a cookie to be passed to[PyIFileOperation::Unadvise](PyIFileOperation.md#pyifileoperationunadvise)to disconnect

## [PyIFileOperation](#pyifileoperation).ApplyPropertiesToItem

 __ApplyPropertiesToItem( *Item* __ )
Specifies the item that will receive property changes

#### Parameters


  -  *Item* :[PyIShellItem](#pyishellitem)

    The item to which property changes will be applied

## [PyIFileOperation](#pyifileoperation).ApplyPropertiesToItems

 __ApplyPropertiesToItems( *Items* __ )
Specifies multiple items that will receive property changes

#### Parameters


  -  *Items* :[PyIUnknown](#pyiunknown)

    [PyIShellItemArray](#pyishellitemarray),[PyIDataObject](#pyidataobject), or[PyIEnumShellItems](#pyienumshellitems)containing the target items

## [PyIFileOperation](#pyifileoperation).CopyItem

 __CopyItem( *Item*  *, DestinationFolder*  *, CopyName*  *, Sink* __ )
Adds a copy operation to the configuration

#### Parameters


  -  *Item* :[PyIShellItem](#pyishellitem)

    Item to be copied

  -  *DestinationFolder* :[PyIShellItem](#pyishellitem)

    Folder into which it will be copied

  -  *CopyName=None* : str

    New name for the copied file, use None to keep original name

  -  *Sink=None* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Progress sink for just this operation

## [PyIFileOperation](#pyifileoperation).CopyItems

 __CopyItems( *Items*  *, DestinationFolder* __ )
Adds multiple copy operations to the configuration

#### Parameters


  -  *Items* :[PyIUnknown](#pyiunknown)

    [PyIShellItemArray](#pyishellitemarray),[PyIDataObject](#pyidataobject), or[PyIEnumShellItems](#pyienumshellitems)containing items to be copied

  -  *DestinationFolder* :[PyIShellItem](#pyishellitem)

    Folder into which they will be copied

## [PyIFileOperation](#pyifileoperation).DeleteItem

 __DeleteItem( *Item*  *, Sink* __ )
Adds a delete operation to the configuration

#### Parameters


  -  *Item* :[PyIShellItem](#pyishellitem)

    Description for psiItem

  -  *Sink=None* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Progress sink for just this operation

## [PyIFileOperation](#pyifileoperation).DeleteItems

 __DeleteItems( *Items* __ )
Adds multiple delete operations to the configuration

#### Parameters


  -  *Items* :[PyIUnknown](#pyiunknown)

    [PyIShellItemArray](#pyishellitemarray),[PyIDataObject](#pyidataobject), or[PyIEnumShellItems](#pyienumshellitems)containing the items to be deleted

## [PyIFileOperation](#pyifileoperation).GetAnyOperationsAborted

boolean = __GetAnyOperationsAborted(__ )
Determines if any operations were terminated

## [PyIFileOperation](#pyifileoperation).MoveItem

 __MoveItem( *Item*  *, DestinationFolder*  *, pszNewName*  *, Sink* __ )
Adds a move operation to the configuration

#### Parameters


  -  *Item* :[PyIShellItem](#pyishellitem)

    The item to be moved

  -  *DestinationFolder* :[PyIShellItem](#pyishellitem)

    The folder into which it will be moved

  -  *pszNewName=None* : str

    Name to be given to moved item, use None to keep original name

  -  *Sink=None* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Progress sink to receive notification for just this operation

## [PyIFileOperation](#pyifileoperation).MoveItems

 __MoveItems( *Items*  *, DestinationFolder* __ )
Adds multiple move operations to the configuration

#### Parameters


  -  *Items* :[PyIUnknown](#pyiunknown)

    [PyIShellItemArray](#pyishellitemarray),[PyIDataObject](#pyidataobject), or[PyIEnumShellItems](#pyienumshellitems)containing the items to be moved

  -  *DestinationFolder* :[PyIShellItem](#pyishellitem)

    Folder into which all items will be moved

## [PyIFileOperation](#pyifileoperation).NewItem

 __NewItem( *DestinationFolder*  *, FileAttributes*  *, Name*  *, TemplateName*  *, Sink* __ )
Creates a new file as part of the operation

#### Parameters


  -  *DestinationFolder* :[PyIShellItem](#pyishellitem)

    Folder in which to create the file

  -  *FileAttributes* : int

    Combination of win32con.FILE_ATTRIBUTE_* flags

  -  *Name* : str

    Name of the new file

  -  *TemplateName=None* : str

    Template file used to initialize the new file

  -  *Sink=None* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Progress sink for just this operation

## [PyIFileOperation](#pyifileoperation).PerformOperations

 __PerformOperations(__ )
Effects all configured file system modifications

## [PyIFileOperation](#pyifileoperation).RenameItem

 __RenameItem( *Item*  *, NewName*  *, Sink* __ )
Adds a rename to the operation sequence

#### Parameters


  -  *Item* :[PyIShellItem](#pyishellitem)

    The item to be renamed

  -  *NewName* : str

    The new name

  -  *Sink=None* :[PyGFileOperationProgressSink](#pygfileoperationprogresssink)

    Progress sink for this operation only.

## [PyIFileOperation](#pyifileoperation).RenameItems

 __RenameItems( *pUnkItems*  *, NewName* __ )
Adds multiple renames to the operation sequence

#### Parameters


  -  *pUnkItems* :[PyIUnknown](#pyiunknown)

    [PyIShellItemArray](#pyishellitemarray),[PyIDataObject](#pyidataobject), or[PyIEnumShellItems](#pyienumshellitems)containing items to be renamed

  -  *NewName* : str

    New name for all items.  Collisions handled automatically.

## [PyIFileOperation](#pyifileoperation).SetOperationFlags

 __SetOperationFlags( *OperationFlags* __ )
Sets option flags for the operation

#### Parameters


  -  *OperationFlags* : int

    Combination of shellcon.FOF_* and FOFX_* flags

## [PyIFileOperation](#pyifileoperation).SetOwnerWindow

 __SetOwnerWindow( *Owner* __ )
Sets the parent window for any UI displayed.

#### Parameters


  -  *Owner* :[PyHANDLE](#pyhandle)

    Handle to parent window

## [PyIFileOperation](#pyifileoperation).SetProgressDialog

 __SetProgressDialog( *popd* __ )
Provides an interface used to display a progress dialog

#### Parameters


  -  *popd* : __PyIOperationsProgressDialog__ 

    Progress dialog interface

#### Comments
IOperationsProgressDialog is not yet supported

## [PyIFileOperation](#pyifileoperation).SetProgressMessage

 __SetProgressMessage( *Message* __ )
Not implemented.

#### Parameters


  -  *Message* : str

    Description for Message

## [PyIFileOperation](#pyifileoperation).SetProperties

 __SetProperties( *proparray* __ )
Specifies a set of properties to be changed.

#### Parameters


  -  *proparray* :[PyIPropertyChangeArray](#pyipropertychangearray)

    Sequence of property changes to be performed (see[propsys::PSCreatePropertyChangeArray](propsys.md#propsyspscreatepropertychangearray))

#### Comments
Note that these properties will be set for *any* files created by the operation, not 

just items passed to ApplyPropertiesToItem(s).  New items created as the result of a 

rename, copy, or move must have a property handler, or the operation fails with the vague
com_error: (-2147467259, 'Unspecified error', None, None) (E_FAIL, or 0x80004005 in hex) 

even though the given file operation was actually performed.

## [PyIFileOperation](#pyifileoperation).Unadvise

 __Unadvise( *Cookie* __ )
Disconnects a progress sink

#### Parameters


  -  *Cookie* : int

    Identifies the sink to disconnect, as returned by[PyIFileOperation::Advise](PyIFileOperation.md#pyifileoperationadvise)