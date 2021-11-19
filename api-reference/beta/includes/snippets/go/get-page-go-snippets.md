---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 902ff43fe09b9361cc1c75623f84570ab1729b02
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083774"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
sitePageId := "sitePage-id"
result, err := graphClient.SitesById(&siteId).PagesById(&sitePageId).Get(options)


```