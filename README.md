# LoadImageAsync

## Usage

```
using Battlehub.Utils;
using UnityEngine;

public class LoadImageAsyncSample : MonoBehaviour
{
    [SerializeField]
    private string m_path;
    
    async void  Start()
    {
        Texture2D texture = new Texture2D(1, 1);
        await texture.LoadImageAsync(m_path);

        Debug.Log($"{texture.width} {texture.height} {texture.format} {texture.mipmapCount}");
    }
}
```

## Plugin source
https://github.com/Battlehub0x/LoadImageAsyncPlugin
