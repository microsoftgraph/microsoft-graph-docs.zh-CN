---
title: 任务中的标识符
description: 任务中的对象标识符是由服务生成的字符串值。 . 这些值的长度为28个字符，区分大小写。 当作为 in 传递时，服务将对标识符进行简单的格式验证，如果格式验证失败，调用方将收到一个错误请求 (400，指示此问题的) 响应。 如果收到此错误，则表示调用应用程序中有一个错误，如：
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: TarkanSevilmis
ms.openlocfilehash: 9ff7b894c8414e2dc7f3dd9d425b0027d0ae13f5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811957"
---
# <a name="identifiers-in-tasks"></a>任务中的标识符

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

任务中的对象标识符是由服务生成的字符串值。 . 这些值的长度为28个字符，区分大小写。 当作为 in 传递时，服务将对标识符进行简单的格式验证，如果格式验证失败，调用方将收到一个错误请求 (400，指示此问题的) 响应。 如果收到此错误，则表示调用应用程序中有一个错误，如：

- 调用应用程序将标识符处理为不区分大小写的字符串。 任务中的标识符区分大小写。
- 调用应用程序截断了标识符。 任务中的标识符长度为28个字符。
- 调用应用程序尝试为任务中的对象生成标识符值。 不接受客户端生成的标识符。 所有标识符都是在创建对象时由服务生成的。

此验证 **不是一项安全功能**。 它仅用于在开发应用程序期间通知应用程序与常见标识符相关的问题，这些问题在其他方面很难识别。
