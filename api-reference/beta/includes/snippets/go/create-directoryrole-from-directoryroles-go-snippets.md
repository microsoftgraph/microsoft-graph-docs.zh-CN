---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cb5732571a07b29ae91aed6d7a40e231606d15b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDirectoryRole()
roleTemplateId := "fe930be7-5e62-47db-91af-98c3a49a38b1"
requestBody.SetRoleTemplateId(&roleTemplateId)
options := &msgraphsdk.DirectoryRolesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryRoles().Post(options)


```