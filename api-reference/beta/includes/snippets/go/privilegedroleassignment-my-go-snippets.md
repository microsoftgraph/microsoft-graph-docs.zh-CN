---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b7def72c5c6c91d8143bcb1d583045b15d7d67e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137762"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedRoleAssignments().My()().Get(nil)


```