---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb8a34a69cab3008e9d555337dbf5f59c11f31cf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088645"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Delete(options)


```