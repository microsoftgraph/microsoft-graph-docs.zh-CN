---
title: Planner 中的标识符
description: Planner 中的对象的标识符是服务生成的字符串值。 值为 28 个字符，且区分大小写。 传入时，服务将执行标识符的简单格式验证，如果格式验证失败，则调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误表示调用应用程序中存在 Bug，例如：
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 4433fc63e884f9c98174a07d7d043f69fce4d8c0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044419"
---
# <a name="identifiers-in-planner"></a>Planner 中的标识符

命名空间：microsoft.graph

Planner 中的对象的标识符是服务生成的字符串值。 值为 28 个字符，且区分大小写。 传入时，服务将执行标识符的简单格式验证，如果格式验证失败，则调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误表示调用应用程序中存在 Bug，例如：

- 调用应用程序将标识符作为不区分大小写的字符串进行处理。 Tasks 中的标识符区分大小写。
- 调用应用程序截断了标识符。 Tasks 中的标识符长 28 个字符。
- 调用应用程序尝试为 Tasks 中的对象生成标识符值。 不接受客户端生成的标识符。 所有标识符由服务在对象创建时生成。

此验证 **不是安全功能**。 它只用于通知应用程序在应用程序开发期间与常见标识符相关的问题，否则很难识别这些问题。

