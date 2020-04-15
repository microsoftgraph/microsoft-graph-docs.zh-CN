---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7f2b3804878b825b0e7eed9a9ed9253abf475f1e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445955"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="fba93-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fba93-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="fba93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fba93-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fba93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba93-106">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="fba93-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="fba93-107">成员</span><span class="sxs-lookup"><span data-stu-id="fba93-107">Members</span></span>
|<span data-ttu-id="fba93-108">成员</span><span class="sxs-lookup"><span data-stu-id="fba93-108">Member</span></span>|<span data-ttu-id="fba93-109">值</span><span class="sxs-lookup"><span data-stu-id="fba93-109">Value</span></span>|<span data-ttu-id="fba93-110">说明</span><span class="sxs-lookup"><span data-stu-id="fba93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba93-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fba93-111">deviceDefault</span></span>|<span data-ttu-id="fba93-112">0</span><span class="sxs-lookup"><span data-stu-id="fba93-112">0</span></span>|<span data-ttu-id="fba93-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="fba93-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fba93-114">无</span><span class="sxs-lookup"><span data-stu-id="fba93-114">none</span></span>|<span data-ttu-id="fba93-115">1</span><span class="sxs-lookup"><span data-stu-id="fba93-115">1</span></span>|<span data-ttu-id="fba93-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="fba93-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="fba93-117">应试</span><span class="sxs-lookup"><span data-stu-id="fba93-117">attempt</span></span>|<span data-ttu-id="fba93-118">双面</span><span class="sxs-lookup"><span data-stu-id="fba93-118">2</span></span>|<span data-ttu-id="fba93-119">仅当支票确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="fba93-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="fba93-120">无须</span><span class="sxs-lookup"><span data-stu-id="fba93-120">require</span></span>|<span data-ttu-id="fba93-121">第三章</span><span class="sxs-lookup"><span data-stu-id="fba93-121">3</span></span>|<span data-ttu-id="fba93-122">在允许证书之前，需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="fba93-122">Require a successful CRL check before allowing a certificate</span></span>|







