---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4465fe428f0d5fc1091b7130b65f81ddde9877be55c26b6f4077d6a036dcfa2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161700"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Tag tag = new Tag();
tag.description = "This is an updated description.";

graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags("e54b3f535b434a9a8743b84e34c00504")
    .buildRequest()
    .patch(tag);

```