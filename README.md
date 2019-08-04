[![Build Status](https://travis-ci.com/linksplatform/Data.Doublets.svg?branch=master)](https://travis-ci.com/linksplatform/Data.Doublets)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/83c66adb68f44a018c795bc7dc7d6f49)](https://app.codacy.com/app/drakonard/Data.Doublets?utm_source=github.com&utm_medium=referral&utm_content=linksplatform/Data.Doublets&utm_campaign=Badge_Grade_Dashboard)
[![CodeFactor](https://www.codefactor.io/repository/github/linksplatform/data.doublets/badge/master)](https://www.codefactor.io/repository/github/linksplatform/data.doublets/overview/master)

# [Data.Doublets](https://github.com/linksplatform/Data.Doublets) ([русская версия](README.ru.md))

LinksPlatform's Platform.Data.Doublets Class Library.

Namespace: [Platform.Data.Doublets](https://linksplatform.github.io/Data.Doublets/api/Platform.Data.Doublets.html)

Forked from: [Konard/LinksPlatform/Platform/Platform.Data.Doublets](https://github.com/Konard/LinksPlatform/tree/b0844d778ced60b22435e57342393031b26a2822/Platform/Platform.Data.Doublets)

NuGet package: [Platform.Data.Doublets](https://www.nuget.org/packages/Platform.Data.Doublets)

## [Example](https://github.com/linksplatform/HelloWorld.Doublets.DotNet)

```C#
using System;
using Platform.Data.Doublets;
using Platform.Data.Doublets.ResizableDirectMemory;

namespace HelloWorld.Doublets.DotNet
{
  class Program
  {
    static void Main()
    {
      using (var links = new ResizableDirectMemoryLinks<uint>("db.links"))
      {
        var link = links.Create();
        link = links.Update(link, link, link);
        Console.WriteLine("Hello World!");
        Console.WriteLine($"This is my first link: ({link}:{links.GetSource(link)}->{links.GetTarget(link)}).");
      }
    }
  }
}
```

## [SQLite vs Doublets](https://github.com/linksplatform/Comparisons.SQLiteVSDoublets)

## [Documentation](https://linksplatform.github.io/Data.Doublets/)

* Interface [ILinks\<TLink, TConstants\>](https://linksplatform.github.io/Data/api/Platform.Data.ILinks-2.html).
* Interface [ILinks\<TLink\>](https://linksplatform.github.io/Data.Doublets/api/Platform.Data.Doublets.ILinks-1.html).
* Class [ResizableDirectMemoryLinks\<TLink\>](https://linksplatform.github.io/Data.Doublets/api/Platform.Data.Doublets.ResizableDirectMemory.ResizableDirectMemoryLinks-1.html).

## Depend on

* [Platform.Collections.Methods](https://github.com/linksplatform/Collections.Methods)
* [Platform.Numbers](https://github.com/linksplatform/Numbers)
* [Platform.Random](https://github.com/linksplatform/Random)
* [Platform.Timestamps](https://github.com/linksplatform/Timestamps)
* [Platform.Helpers](https://github.com/linksplatform/Helpers)
* [Platform.Memory](https://github.com/linksplatform/Memory)
* [Platform.Data](https://github.com/linksplatform/Data)