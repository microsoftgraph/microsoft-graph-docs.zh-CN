---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c60d713ea25dcc5a2488198396afb487774850de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961706"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().homeRealmDiscoveryPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```