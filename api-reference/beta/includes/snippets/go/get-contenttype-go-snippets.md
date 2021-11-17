---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54e67ca47c237931d2b5843f2017abb069dc54a4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Get(options)


```