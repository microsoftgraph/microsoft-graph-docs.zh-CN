---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d9e4a6c4b1a68a614b1fae692ad8bab4d4034cbd2dd359351c71957b4ad933d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277539"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .delete();

```