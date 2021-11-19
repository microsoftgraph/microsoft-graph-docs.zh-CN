---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff3c6b5a27e5dce05d0b1fb6c9ede35f80cfb075
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
graphClient.TeamsById(&teamId).Archive().Post(options)


```