---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3fa77e067d410cf25944a90c04e5901b3c245e60c3a6d03ab64f76e24e60139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105787"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TagAsHierarchyCollectionPage asHierarchy = graphClient.compliance().ediscovery().cases("47746044-fd0b-4a30-acfc-5272b691ba5b").tags()
    .asHierarchy()
    .buildRequest()
    .get();

```