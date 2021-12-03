---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a32409ce41cc456a180ffaf2a82f43d65ef2bed
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288653"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
groupId := "group-id"
graphClient.SitesById(&siteId).TermStore().GroupsById(&groupId).Delete(nil)


```