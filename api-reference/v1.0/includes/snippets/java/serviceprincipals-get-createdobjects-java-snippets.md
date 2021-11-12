---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 948846753b8eb8755a2730d767d7b0845bf3c1827caea6adc83a23372394e021
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103773"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage createdObjects = graphClient.servicePrincipals("{id}").createdObjects()
    .buildRequest()
    .get();

```