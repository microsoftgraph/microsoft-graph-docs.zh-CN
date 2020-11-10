---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88d020ba1509f00cd7f396caa37341329a0fe096
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982234"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISchemaExtensionCollectionPage schemaExtensions = graphClient.schemaExtensions()
    .buildRequest()
    .filter("id eq 'graphlearn_test'")
    .get();

```