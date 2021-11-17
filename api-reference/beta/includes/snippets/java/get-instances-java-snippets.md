---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d7f8820502a4b4420a82dfaf11eaf1eff551f47060a92d1f3d7f996540dff52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2019-04-08T09:00:00.0000000"));
requestOptions.add(new QueryOption("endDateTime", "2019-04-30T09:00:00.0000000"));

EventCollectionPage instances = graphClient.me().events("AAMkAGUzYRgWAAA=").instances()
    .buildRequest( requestOptions )
    .select("subject,bodyPreview,seriesMasterId,type,recurrence,start,end")
    .get();

```