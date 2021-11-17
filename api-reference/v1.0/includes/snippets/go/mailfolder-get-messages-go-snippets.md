---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d336f521a21fd3dcc01d89d0a60d333dd7f577cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029496"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Messages().Get(options)


```