---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc14b2cf8843171e7ac8160028cee2996c055a5a
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224590"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters{
    Filter: "attributeSet%20eq%20'Engineering'%20and%20status%20eq%20'Available'%20and%20type%20eq%20'String'",
}
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Get(options)


```