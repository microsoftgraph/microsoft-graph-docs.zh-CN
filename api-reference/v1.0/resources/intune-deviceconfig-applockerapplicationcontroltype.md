---
title: appLockerApplicationControlType 枚举类型
description: AppLocker 应用程序控件类型的可能值
ms.openlocfilehash: 703cc18dfee49a01adb3cd4f61c5d7e99e30fb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008170"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="8963c-103">appLockerApplicationControlType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8963c-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="8963c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8963c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8963c-105">AppLocker 应用程序控件类型的可能值</span><span class="sxs-lookup"><span data-stu-id="8963c-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="8963c-106">成员</span><span class="sxs-lookup"><span data-stu-id="8963c-106">Members</span></span>
|<span data-ttu-id="8963c-107">成员</span><span class="sxs-lookup"><span data-stu-id="8963c-107">Member</span></span>|<span data-ttu-id="8963c-108">值</span><span class="sxs-lookup"><span data-stu-id="8963c-108">Value</span></span>|<span data-ttu-id="8963c-109">说明</span><span class="sxs-lookup"><span data-stu-id="8963c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8963c-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8963c-110">notConfigured</span></span>|<span data-ttu-id="8963c-111">0</span><span class="sxs-lookup"><span data-stu-id="8963c-111">0</span></span>|<span data-ttu-id="8963c-112">设备默认值，未选择的应用程序控制类型。</span><span class="sxs-lookup"><span data-stu-id="8963c-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="8963c-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="8963c-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="8963c-114">1</span><span class="sxs-lookup"><span data-stu-id="8963c-114">1</span></span>|<span data-ttu-id="8963c-115">强制实施 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8963c-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="8963c-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="8963c-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="8963c-117">2</span><span class="sxs-lookup"><span data-stu-id="8963c-117">2</span></span>|<span data-ttu-id="8963c-118">审核 Windows 组件和 store 应用程序。</span><span class="sxs-lookup"><span data-stu-id="8963c-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="8963c-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="8963c-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="8963c-120">3</span><span class="sxs-lookup"><span data-stu-id="8963c-120">3</span></span>|<span data-ttu-id="8963c-121">强制实施 Windows 组件、 存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="8963c-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="8963c-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="8963c-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="8963c-123">4</span><span class="sxs-lookup"><span data-stu-id="8963c-123">4</span></span>|<span data-ttu-id="8963c-124">审核 Windows 组件，存储应用程序和智能锁定者。</span><span class="sxs-lookup"><span data-stu-id="8963c-124">Audit Windows components, store apps and smart locker.</span></span>|



