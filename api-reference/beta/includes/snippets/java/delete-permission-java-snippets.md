---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aee750c1a4d2c276bd66a8815055a96e681793d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973025"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().items().{item-id}().permissions().{perm-id}()
    .buildRequest()
    .delete();

```