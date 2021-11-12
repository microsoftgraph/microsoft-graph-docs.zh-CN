---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f971e138ef9bad919f82981116bc32d1b3c075458eec72edc8f1cf955e8f288f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215660"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.applications("{id}").owners()
    .buildRequest()
    .get();

```