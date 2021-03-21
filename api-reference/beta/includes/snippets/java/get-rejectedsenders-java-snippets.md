---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25dbfefeb0f6b72a9c9ac6d9ff0d2483b15f8802
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970228"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage rejectedSenders = graphClient.groups("{id}").rejectedSenders()
    .buildRequest()
    .get();

```