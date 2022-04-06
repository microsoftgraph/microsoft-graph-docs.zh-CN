---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9185a7b80b15dfd626c03ed46db8cb187a867449
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528098"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Delete(nil)


```