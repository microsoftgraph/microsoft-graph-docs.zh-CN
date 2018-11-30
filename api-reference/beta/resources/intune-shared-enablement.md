---
title: 启用枚举类型
description: '用于指示状态的设备的值。 '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045101"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="659fd-103">启用枚举类型</span><span class="sxs-lookup"><span data-stu-id="659fd-103">enablement enum type</span></span>

> <span data-ttu-id="659fd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="659fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="659fd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="659fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="659fd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="659fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="659fd-107">用于指示状态的设备的值。</span><span class="sxs-lookup"><span data-stu-id="659fd-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="659fd-108">请注意，没有区别禁用，且未配置。</span><span class="sxs-lookup"><span data-stu-id="659fd-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="659fd-109">成员</span><span class="sxs-lookup"><span data-stu-id="659fd-109">Members</span></span>
|<span data-ttu-id="659fd-110">成员</span><span class="sxs-lookup"><span data-stu-id="659fd-110">Member</span></span>|<span data-ttu-id="659fd-111">值</span><span class="sxs-lookup"><span data-stu-id="659fd-111">Value</span></span>|<span data-ttu-id="659fd-112">说明</span><span class="sxs-lookup"><span data-stu-id="659fd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="659fd-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="659fd-113">notConfigured</span></span>|<span data-ttu-id="659fd-114">0</span><span class="sxs-lookup"><span data-stu-id="659fd-114">0</span></span>|<span data-ttu-id="659fd-115">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="659fd-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="659fd-116">enabled</span><span class="sxs-lookup"><span data-stu-id="659fd-116">enabled</span></span>|<span data-ttu-id="659fd-117">1</span><span class="sxs-lookup"><span data-stu-id="659fd-117">1</span></span>|<span data-ttu-id="659fd-118">允许在设备上的设置。</span><span class="sxs-lookup"><span data-stu-id="659fd-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="659fd-119">禁用</span><span class="sxs-lookup"><span data-stu-id="659fd-119">disabled</span></span>|<span data-ttu-id="659fd-120">2</span><span class="sxs-lookup"><span data-stu-id="659fd-120">2</span></span>|<span data-ttu-id="659fd-121">禁用在设备上的设置。</span><span class="sxs-lookup"><span data-stu-id="659fd-121">Disables the setting on the device.</span></span>|
