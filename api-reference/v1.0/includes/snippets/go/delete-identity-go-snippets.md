---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e783c0e53fb2c3477cbe03c8a100b19a74047370
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329044"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
identityId := "identity-id"
graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).MembersById(&identityId).Delete()


```