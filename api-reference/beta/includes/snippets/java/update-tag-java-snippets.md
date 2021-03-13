---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34cf9acad9c5f81a61f9923a65540100a819235b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776401"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tag tag = new Tag();
tag.description = "This is an updated description.";

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("e54b3f535b434a9a8743b84e34c00504")
    .buildRequest()
    .patch(tag);

```