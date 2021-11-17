---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4805902523d26c0545c117e799d6aabd57bc77d2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024861"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
endpointId := "endpoint-id"
result, err := graphClient.GroupsById(&groupId).EndpointsById(&endpointId).Get(options)


```