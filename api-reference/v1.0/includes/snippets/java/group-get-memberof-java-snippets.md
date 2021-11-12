---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660abaee5c733a79cf4d1ea5d525a79f416248a6861b723b3cdbf3f5a891bcd8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162988"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.groups("{id}").memberOf()
    .buildRequest()
    .get();

```