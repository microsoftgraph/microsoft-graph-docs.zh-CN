---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持管理条件表达式二元运算符。
ms.openlocfilehash: e1f58715f4e900c30a52bbe7a9db01e45a081d09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049030"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="91e27-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="91e27-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="91e27-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91e27-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91e27-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91e27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91e27-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91e27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91e27-107">支持管理条件表达式二元运算符。</span><span class="sxs-lookup"><span data-stu-id="91e27-107">Supported binary operators for management condition expressions.</span></span>
## <a name="members"></a><span data-ttu-id="91e27-108">成员</span><span class="sxs-lookup"><span data-stu-id="91e27-108">Members</span></span>
|<span data-ttu-id="91e27-109">成员</span><span class="sxs-lookup"><span data-stu-id="91e27-109">Member</span></span>|<span data-ttu-id="91e27-110">值</span><span class="sxs-lookup"><span data-stu-id="91e27-110">Value</span></span>|<span data-ttu-id="91e27-111">说明</span><span class="sxs-lookup"><span data-stu-id="91e27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e27-112">或</span><span class="sxs-lookup"><span data-stu-id="91e27-112">or</span></span>|<span data-ttu-id="91e27-113">0</span><span class="sxs-lookup"><span data-stu-id="91e27-113">0</span></span>|<span data-ttu-id="91e27-114">计算一操作数为 true，当且仅当一个或多个操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="91e27-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="91e27-115">和</span><span class="sxs-lookup"><span data-stu-id="91e27-115">and</span></span>|<span data-ttu-id="91e27-116">1</span><span class="sxs-lookup"><span data-stu-id="91e27-116">1</span></span>|<span data-ttu-id="91e27-117">当且仅当所有的操作数，则，计算一操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="91e27-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





