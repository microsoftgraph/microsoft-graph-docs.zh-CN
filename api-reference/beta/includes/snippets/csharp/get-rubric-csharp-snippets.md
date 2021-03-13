---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e154a2aff5dadc2f112e3320f803337e112b6023
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801556"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Me.Assignments["{educationAssignment-id}"].Rubric
    .Request()
    .GetAsync();

```