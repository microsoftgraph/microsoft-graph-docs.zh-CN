---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 127585b9a94822dd6ceaf868e35dc7cb03a20afa19f8921944a160f53d32171b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

Event event = graphClient.me().events("AAMkAGIAAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees")
    .get();

```