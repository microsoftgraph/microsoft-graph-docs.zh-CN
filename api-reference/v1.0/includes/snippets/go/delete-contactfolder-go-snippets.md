---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdc2a37b505d5e5833b616112a5d90d19e2ce6bc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974325"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

contactFolderId := "contactFolder-id"
graphClient.Me().ContactFoldersById(&contactFolderId).Delete(options)


```