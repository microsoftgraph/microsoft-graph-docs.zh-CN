---
title: 任务中的标识符
description: 任务中对象的标识符是服务生成的字符串值。 . 这些值长 28 个字符，区分大小写。 当传入时，服务将对标识符执行简单的格式验证，如果格式验证失败，调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示调用应用程序中的 bug，例如：
ms.localizationpriority: medium
doc_type: conceptualPageType
ms.prod: tasks-and-plans
author: TarkanSevilmis
ms.openlocfilehash: 4bac8d2fca466da934ac55b16c09c6c1d0977d32
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732693"
---
# <a name="identifiers-in-tasks"></a>任务中的标识符

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

任务中对象的标识符是服务生成的字符串值。 . 这些值长 28 个字符，区分大小写。 当传入时，服务将对标识符执行简单的格式验证，如果格式验证失败，调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误指示调用应用程序中的 bug，例如：

- 调用应用程序将标识符处理为不区分大小写的字符串。 任务中的标识符区分大小写。
- 调用应用程序截断了标识符。 任务中的标识符长度为 28 个字符。
- 调用应用程序尝试为 Tasks 中的对象生成标识符值。 不接受客户端生成的标识符。 创建对象时，服务会生成所有标识符。

此验证 **不是安全功能**。 它仅用于在应用程序开发过程中告知应用程序常见标识符相关问题，否则难以识别。


