---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4db8f63f338d4c695379493f2c1753852f7e1f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983680"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().contacts("{id}")
    .buildRequest()
    .delete();

```