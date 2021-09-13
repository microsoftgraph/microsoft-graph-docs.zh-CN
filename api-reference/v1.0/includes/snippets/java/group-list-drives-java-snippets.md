---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8371b136d77592d6304f37709eb95cb4123dbfdca5e028bd1e318d7ddf836159
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.groups("{groupId}").drives()
    .buildRequest()
    .get();

```