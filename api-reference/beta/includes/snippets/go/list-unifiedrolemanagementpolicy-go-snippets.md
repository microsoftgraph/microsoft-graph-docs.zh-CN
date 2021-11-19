---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef4ec2c10ee55f4075fe9bb32b2ce406ba469eb7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091571"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().RoleManagementPolicies().Get(options)


```