---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持的管理条件表达式的二元运算符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35f60b9ee321ef3cbd65cf77273a65e7705f666a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143804"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="6704f-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6704f-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="6704f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6704f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6704f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6704f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6704f-106">支持的管理条件表达式的二元运算符。</span><span class="sxs-lookup"><span data-stu-id="6704f-106">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="6704f-107">成员</span><span class="sxs-lookup"><span data-stu-id="6704f-107">Members</span></span>
|<span data-ttu-id="6704f-108">成员</span><span class="sxs-lookup"><span data-stu-id="6704f-108">Member</span></span>|<span data-ttu-id="6704f-109">值</span><span class="sxs-lookup"><span data-stu-id="6704f-109">Value</span></span>|<span data-ttu-id="6704f-110">说明</span><span class="sxs-lookup"><span data-stu-id="6704f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6704f-111">或</span><span class="sxs-lookup"><span data-stu-id="6704f-111">or</span></span>|<span data-ttu-id="6704f-112">0</span><span class="sxs-lookup"><span data-stu-id="6704f-112">0</span></span>|<span data-ttu-id="6704f-113">当且仅当一个或多个操作数为 true 时, 将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="6704f-113">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="6704f-114">和</span><span class="sxs-lookup"><span data-stu-id="6704f-114">and</span></span>|<span data-ttu-id="6704f-115">1</span><span class="sxs-lookup"><span data-stu-id="6704f-115">1</span></span>|<span data-ttu-id="6704f-116">当且仅当其所有操作数均为 true 时, 将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="6704f-116">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|




