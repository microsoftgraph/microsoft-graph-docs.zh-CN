---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0966ddf2c4d653470c7de57dddea205d78fd716e32f3d2b77f7975fb9dc9e571
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExtensionPropertyCollectionPage extensionProperties = graphClient.applications("{id}").extensionProperties()
    .buildRequest()
    .get();

```