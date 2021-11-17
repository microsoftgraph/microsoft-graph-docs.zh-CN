---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 781f4674a9d80e3dc6193848fb0ed824ce9df3be
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997659"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

personWebsiteId := "personWebsite-id"
result, err := graphClient.Me().Profile().WebsitesById(&personWebsiteId).Get(options)


```