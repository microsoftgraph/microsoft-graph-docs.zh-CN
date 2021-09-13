---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80e1bcfaa41ec908f122927878269b3858eacc5fad52032247cad86a4b1d3a13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220390"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToSectionGroup(OnenoteSectionCopyToSectionGroupParameterSet
        .newBuilder()
        .withId(id)
        .withGroupId(groupId)
        .withRenameAs(renameAs)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```