# PlayModeComponentSaver
保存播放模式下所做的数据更改

只是修复了 Assets Store [Play Mode Saver](https://assetstore.unity.com/packages/tools/utilities/play-mode-saver-104836)  插件在 Unity 6 下的一个Bug

```c#
if (_clearButtonContent == null)
{
   // Unity 6 下会报错
   // _clearButtonContent = EditorGUIUtility.IconContent("d_winbtn_win_close");
   // _clearButtonContent = EditorGUIUtility.IconContent("d_winbtn_mac_close");
   _clearButtonContent = EditorGUIUtility.IconContent("Close");
}
```
