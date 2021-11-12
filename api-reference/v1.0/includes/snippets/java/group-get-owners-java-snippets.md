---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbef3fd04cec5cca93f4bba3f17cda46a672fe96a8d217e3a9e238d9d789ddf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage owners = graphClient.groups("{id}").owners()
    .buildRequest()
    .get();

```