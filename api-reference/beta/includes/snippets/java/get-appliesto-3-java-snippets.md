---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 163fec1c414929a8b3bfdd20d446c454dcab4bea
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208991"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().tokenIssuancePolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```