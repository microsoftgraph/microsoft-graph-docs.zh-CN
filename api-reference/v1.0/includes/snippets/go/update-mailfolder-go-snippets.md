---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76fe889afed5f993364986387bed460f1351f4eb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104001"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

mailFolderId := "mailFolder-id"
graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```