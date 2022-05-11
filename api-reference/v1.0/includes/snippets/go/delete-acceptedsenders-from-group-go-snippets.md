---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 738573dd69cb87c6276accde7a7a0164c7fd3074
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderDeleteRequestConfiguration{
    QueryParameters: requestParameters,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).AcceptedSendersById(&directoryObjectId).DeleteWithRequestConfigurationAndResponseHandler(options, nil)


```