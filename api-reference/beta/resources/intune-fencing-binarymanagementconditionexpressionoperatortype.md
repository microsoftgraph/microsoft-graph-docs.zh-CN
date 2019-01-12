---
title: binaryManagementConditionExpressionOperatorType 枚举类型
description: 支持管理条件表达式二元运算符。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 141238fd90b6cae65ac50745d950d3d9d149280d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959410"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="71341-103">binaryManagementConditionExpressionOperatorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="71341-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="71341-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="71341-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71341-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="71341-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71341-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="71341-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71341-107">支持管理条件表达式二元运算符。</span><span class="sxs-lookup"><span data-stu-id="71341-107">Supported binary operators for management condition expressions.</span></span>
## <a name="members"></a><span data-ttu-id="71341-108">成员</span><span class="sxs-lookup"><span data-stu-id="71341-108">Members</span></span>
|<span data-ttu-id="71341-109">成员</span><span class="sxs-lookup"><span data-stu-id="71341-109">Member</span></span>|<span data-ttu-id="71341-110">值</span><span class="sxs-lookup"><span data-stu-id="71341-110">Value</span></span>|<span data-ttu-id="71341-111">Description</span><span class="sxs-lookup"><span data-stu-id="71341-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71341-112">或</span><span class="sxs-lookup"><span data-stu-id="71341-112">or</span></span>|<span data-ttu-id="71341-113">0</span><span class="sxs-lookup"><span data-stu-id="71341-113">0</span></span>|<span data-ttu-id="71341-114">计算一操作数为 true，当且仅当一个或多个操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="71341-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="71341-115">和</span><span class="sxs-lookup"><span data-stu-id="71341-115">and</span></span>|<span data-ttu-id="71341-116">1</span><span class="sxs-lookup"><span data-stu-id="71341-116">1</span></span>|<span data-ttu-id="71341-117">当且仅当所有的操作数，则，计算一操作数为 true。</span><span class="sxs-lookup"><span data-stu-id="71341-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





