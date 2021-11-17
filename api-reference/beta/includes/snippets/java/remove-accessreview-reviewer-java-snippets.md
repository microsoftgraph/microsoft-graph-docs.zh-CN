---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fedd2d64b4afa10455fa2320b99bcb76e971bde4ec2e1288f5cf2e31fe3627ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2b83cc42-09db-46f6-8c6e-16fec466a82d").reviewers("006111db-0810-4494-a6df-904d368bd81b")
    .buildRequest()
    .delete();

```