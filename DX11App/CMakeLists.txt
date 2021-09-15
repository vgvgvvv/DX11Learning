

set(targetName DX11App)
ReMake_AddTarget(
        TARGET_NAME ${targetName}
        MODE EXE
        LIB ResetCore_Framework
            ResetCore_CommonLib
)

WithWinMain(${targetName})

ReMake_StartUse()
UseDirectX11(${targetName})
ReMake_EndUse()