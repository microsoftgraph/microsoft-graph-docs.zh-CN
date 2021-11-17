---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 098b2fdd639716947200e664f4c933121ea17007
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007389"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

programId := "program-id"
graphClient.ProgramsById(&programId).Delete(options)


```