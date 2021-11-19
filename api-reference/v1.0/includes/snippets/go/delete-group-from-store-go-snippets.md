---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b72ab209d545ebf57630dd45bf26f9d32b97dd9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090676"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Delete(options)


```