---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a3d16ad68bbbbb27c904cba8d61ee6ceaac4fa6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966598"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().assignments("{id}").rubric().reference()
    .buildRequest()
    .delete();

```