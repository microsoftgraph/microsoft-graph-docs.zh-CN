---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb9335ee90b8e36a0065fd2b56a301914d15b980
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959374"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICertificateBasedAuthConfigurationCollectionWithReferencesPage certificateBasedAuthConfiguration = graphClient.organization("{id}").certificateBasedAuthConfiguration()
    .buildRequest()
    .get();

```