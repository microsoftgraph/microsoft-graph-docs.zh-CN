---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27220b8f966b3e7b8dc5252e9e0a4d0608ae8cbe
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014082"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
sitePageId := "sitePage-id"
result, err := graphClient.SitesById(&siteId).PagesById(&sitePageId).Get(options)


```