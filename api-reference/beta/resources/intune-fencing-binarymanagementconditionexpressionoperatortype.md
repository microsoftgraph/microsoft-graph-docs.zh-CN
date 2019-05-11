---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持的管理条件表达式的二元运算符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca2518b554388fdd00fae8310ac14c105f5b62ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941308"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="df321-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df321-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="df321-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df321-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df321-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df321-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df321-106">支持的管理条件表达式的二元运算符。</span><span class="sxs-lookup"><span data-stu-id="df321-106">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="df321-107">成员</span><span class="sxs-lookup"><span data-stu-id="df321-107">Members</span></span>
|<span data-ttu-id="df321-108">成员</span><span class="sxs-lookup"><span data-stu-id="df321-108">Member</span></span>|<span data-ttu-id="df321-109">值</span><span class="sxs-lookup"><span data-stu-id="df321-109">Value</span></span>|<span data-ttu-id="df321-110">说明</span><span class="sxs-lookup"><span data-stu-id="df321-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df321-111">或</span><span class="sxs-lookup"><span data-stu-id="df321-111">or</span></span>|<span data-ttu-id="df321-112">0</span><span class="sxs-lookup"><span data-stu-id="df321-112">0</span></span>|<span data-ttu-id="df321-113">当且仅当一个或多个操作数为 true 时, 将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="df321-113">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="df321-114">和</span><span class="sxs-lookup"><span data-stu-id="df321-114">and</span></span>|<span data-ttu-id="df321-115">1</span><span class="sxs-lookup"><span data-stu-id="df321-115">1</span></span>|<span data-ttu-id="df321-116">当且仅当其所有操作数均为 true 时, 将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="df321-116">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|




