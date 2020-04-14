---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持的管理条件表达式的二元运算符。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b007a3d6e673ff3a8d08454eedc0e3f7473d94e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382807"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="1d26c-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1d26c-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

<span data-ttu-id="1d26c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d26c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d26c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d26c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d26c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d26c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d26c-107">支持的管理条件表达式的二元运算符。</span><span class="sxs-lookup"><span data-stu-id="1d26c-107">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="1d26c-108">成员</span><span class="sxs-lookup"><span data-stu-id="1d26c-108">Members</span></span>
|<span data-ttu-id="1d26c-109">成员</span><span class="sxs-lookup"><span data-stu-id="1d26c-109">Member</span></span>|<span data-ttu-id="1d26c-110">值</span><span class="sxs-lookup"><span data-stu-id="1d26c-110">Value</span></span>|<span data-ttu-id="1d26c-111">说明</span><span class="sxs-lookup"><span data-stu-id="1d26c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d26c-112">或</span><span class="sxs-lookup"><span data-stu-id="1d26c-112">or</span></span>|<span data-ttu-id="1d26c-113">0</span><span class="sxs-lookup"><span data-stu-id="1d26c-113">0</span></span>|<span data-ttu-id="1d26c-114">当且仅当一个或多个操作数为 true 时，将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="1d26c-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="1d26c-115">和</span><span class="sxs-lookup"><span data-stu-id="1d26c-115">and</span></span>|<span data-ttu-id="1d26c-116">1</span><span class="sxs-lookup"><span data-stu-id="1d26c-116">1</span></span>|<span data-ttu-id="1d26c-117">当且仅当其所有操作数均为 true 时，将一组操作数评估为 true。</span><span class="sxs-lookup"><span data-stu-id="1d26c-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|



