---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aec65eaa29c4edb729e1ce9dbc83d5ed09678b48
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
endpointId := "endpoint-id"
result, err := graphClient.GroupsById(&groupId).EndpointsById(&endpointId).Get(options)


```