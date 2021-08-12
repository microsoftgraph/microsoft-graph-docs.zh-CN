---
title: Planner 中的标识符
description: Planner 中的对象的标识符是服务生成的字符串值。 值为 28 个字符，且区分大小写。 传入时，服务将执行标识符的简单格式验证，如果格式验证失败，则调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误表示调用应用程序中存在 Bug，例如：
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: 97381d57e8f23b6f032cdf0ebfc02a5cdf32ca2219a1d7c8127e472666250c58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202159"
---
# <a name="identifiers-in-planner"></a>Planner 中的标识符

命名空间：microsoft.graph

Planner 中的对象的标识符是服务生成的字符串值。 值为 28 个字符，且区分大小写。 传入时，服务将执行标识符的简单格式验证，如果格式验证失败，则调用方将收到错误请求 (400) 错误响应，指示此问题。 收到此错误表示调用应用程序中存在 Bug，例如：

- 调用应用程序将标识符作为不区分大小写的字符串进行处理。 Tasks 中的标识符区分大小写。
- 调用应用程序截断了标识符。 Tasks 中的标识符长 28 个字符。
- 调用应用程序尝试为 Tasks 中的对象生成标识符值。 不接受客户端生成的标识符。 所有标识符由服务在对象创建时生成。

此验证 **不是安全功能**。 它只用于通知应用程序在应用程序开发期间与常见标识符相关的问题，否则很难识别这些问题。

