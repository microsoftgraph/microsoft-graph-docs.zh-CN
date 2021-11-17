---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 899f0eb5cb51f0a45832e8807de67e9ab0e12ca421a0b02e3b71efbf49af3e49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105078"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage createdObjects = graphClient.me().createdObjects()
    .buildRequest()
    .get();

```