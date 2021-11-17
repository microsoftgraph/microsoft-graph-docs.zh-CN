---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d3db57442b1993dc995b522e7af9d0081fbffda
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973940"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewDirectoryRole()
roleTemplateId := "fe930be7-5e62-47db-91af-98c3a49a38b1"
requestBody.SetRoleTemplateId(&roleTemplateId)
options := &msgraphsdk.DirectoryRolesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryRoles().Post(options)


```