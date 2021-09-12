---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96ec8b6d0f8d81428307fbeafecbaebc2f74bc786ebf898484b93c7c1c91a9ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274438"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().sectionGroups("{id}").sectionGroups()
    .buildRequest()
    .get();

```