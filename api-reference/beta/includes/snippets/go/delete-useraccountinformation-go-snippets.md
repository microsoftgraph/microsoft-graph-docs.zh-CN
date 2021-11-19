---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ed8ef29aab5c6fcf8500dec477ca10fdcb1092e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088437"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userAccountInformationId := "userAccountInformation-id"
graphClient.Me().Profile().AccountById(&userAccountInformationId).Delete(options)


```