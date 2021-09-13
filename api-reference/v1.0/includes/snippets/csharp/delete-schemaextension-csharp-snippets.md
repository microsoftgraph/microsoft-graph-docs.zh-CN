---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fbc318621debcfc1defc2782a16d27ff46b2bee62daed58bb72b6786b352d9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .DeleteAsync();

```