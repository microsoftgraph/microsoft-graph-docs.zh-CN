---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fca9cea1576509a85695a2c096f01c3da9585c6a4bc238fd0d71e81e7920b4e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtensionCollectionPage schemaExtensions = graphClient.schemaExtensions()
    .buildRequest()
    .filter("id eq 'graphlearn_test'")
    .get();

```