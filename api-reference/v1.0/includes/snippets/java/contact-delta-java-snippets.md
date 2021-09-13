---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 793ba1944b2602dd9dc52a7b91cec5534860954654f1331e605b241212c3a9f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328899"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));

ContactDeltaCollectionPage delta = graphClient.me().contactFolders("{id}").contacts()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName")
    .get();

```