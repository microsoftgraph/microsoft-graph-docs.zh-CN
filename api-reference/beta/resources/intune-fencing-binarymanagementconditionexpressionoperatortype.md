---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持管理条件表达式二元运算符。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05b195df95d6f7a85673a352edf090cea7f074aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424292"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="43c9e-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="43c9e-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="43c9e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="43c9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43c9e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="43c9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43c9e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43c9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c9e-107">支持管理条件表达式二元运算符。</span><span class="sxs-lookup"><span data-stu-id="43c9e-107">Supported binary operators for management condition expressions.</span></span>

## <a name="members"></a><span data-ttu-id="43c9e-108">成员</span><span class="sxs-lookup"><span data-stu-id="43c9e-108">Members</span></span>
|<span data-ttu-id="43c9e-109">成员</span><span class="sxs-lookup"><span data-stu-id="43c9e-109">Member</span></span>|<span data-ttu-id="43c9e-110">值</span><span class="sxs-lookup"><span data-stu-id="43c9e-110">Value</span></span>|<span data-ttu-id="43c9e-111">说明</span><span class="sxs-lookup"><span data-stu-id="43c9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43c9e-112">或</span><span class="sxs-lookup"><span data-stu-id="43c9e-112">or</span></span>|<span data-ttu-id="43c9e-113">0</span><span class="sxs-lookup"><span data-stu-id="43c9e-113">0</span></span>|<span data-ttu-id="43c9e-114">计算一操作数为 true，当且仅当一个或多个操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="43c9e-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="43c9e-115">和</span><span class="sxs-lookup"><span data-stu-id="43c9e-115">and</span></span>|<span data-ttu-id="43c9e-116">1</span><span class="sxs-lookup"><span data-stu-id="43c9e-116">1</span></span>|<span data-ttu-id="43c9e-117">当且仅当所有的操作数，则，计算一操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="43c9e-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|




