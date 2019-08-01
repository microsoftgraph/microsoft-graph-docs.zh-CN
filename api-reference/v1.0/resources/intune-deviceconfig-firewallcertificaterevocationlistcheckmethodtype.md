---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7c5fa3baaeb3d24bc902d733a6c6462fbcf70f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028299"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="86659-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="86659-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="86659-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86659-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86659-105">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="86659-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="86659-106">成员</span><span class="sxs-lookup"><span data-stu-id="86659-106">Members</span></span>
|<span data-ttu-id="86659-107">成员</span><span class="sxs-lookup"><span data-stu-id="86659-107">Member</span></span>|<span data-ttu-id="86659-108">值</span><span class="sxs-lookup"><span data-stu-id="86659-108">Value</span></span>|<span data-ttu-id="86659-109">说明</span><span class="sxs-lookup"><span data-stu-id="86659-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86659-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="86659-110">deviceDefault</span></span>|<span data-ttu-id="86659-111">0</span><span class="sxs-lookup"><span data-stu-id="86659-111">0</span></span>|<span data-ttu-id="86659-112">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="86659-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="86659-113">无</span><span class="sxs-lookup"><span data-stu-id="86659-113">none</span></span>|<span data-ttu-id="86659-114">1</span><span class="sxs-lookup"><span data-stu-id="86659-114">1</span></span>|<span data-ttu-id="86659-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="86659-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="86659-116">应试</span><span class="sxs-lookup"><span data-stu-id="86659-116">attempt</span></span>|<span data-ttu-id="86659-117">双面</span><span class="sxs-lookup"><span data-stu-id="86659-117">2</span></span>|<span data-ttu-id="86659-118">仅当支票确认证书时, 才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="86659-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="86659-119">无须</span><span class="sxs-lookup"><span data-stu-id="86659-119">require</span></span>|<span data-ttu-id="86659-120">第三章</span><span class="sxs-lookup"><span data-stu-id="86659-120">3</span></span>|<span data-ttu-id="86659-121">在允许证书之前, 需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="86659-121">Require a successful CRL check before allowing a certificate</span></span>|



