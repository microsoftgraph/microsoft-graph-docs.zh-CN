---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dd4cf0cffc23025d522f5aed15714f1eaefe5f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038233"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinitionCollectionPage columns = graphClient.sites("{site-id}").contentTypes("{contentType-id}").columns()
    .buildRequest()
    .get();

```