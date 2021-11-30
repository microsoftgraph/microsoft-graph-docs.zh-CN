---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aa180781e96cca632f367bce73e8bf01b490afd
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters{
    Filter: "name%20eq%20'Project'%20and%20status%20eq%20'Available'",
}
options := &msgraphsdk.CustomSecurityAttributeDefinitionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Directory().CustomSecurityAttributeDefinitions().Get(options)


```