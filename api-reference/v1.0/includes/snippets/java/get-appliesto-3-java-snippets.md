---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae661b27c7cc48c42a2851846e877f891d2b3705fba778fa248f61952f2cd963
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenIssuancePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```