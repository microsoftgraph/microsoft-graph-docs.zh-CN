---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: firewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257629"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="2277f-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2277f-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="2277f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2277f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2277f-105">firewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="2277f-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="2277f-106">成员</span><span class="sxs-lookup"><span data-stu-id="2277f-106">Members</span></span>
|<span data-ttu-id="2277f-107">成员</span><span class="sxs-lookup"><span data-stu-id="2277f-107">Member</span></span>|<span data-ttu-id="2277f-108">值</span><span class="sxs-lookup"><span data-stu-id="2277f-108">Value</span></span>|<span data-ttu-id="2277f-109">说明</span><span class="sxs-lookup"><span data-stu-id="2277f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2277f-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2277f-110">deviceDefault</span></span>|<span data-ttu-id="2277f-111">0</span><span class="sxs-lookup"><span data-stu-id="2277f-111">0</span></span>|<span data-ttu-id="2277f-112">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="2277f-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2277f-113">无</span><span class="sxs-lookup"><span data-stu-id="2277f-113">none</span></span>|<span data-ttu-id="2277f-114">1</span><span class="sxs-lookup"><span data-stu-id="2277f-114">1</span></span>|<span data-ttu-id="2277f-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="2277f-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="2277f-116">应试</span><span class="sxs-lookup"><span data-stu-id="2277f-116">attempt</span></span>|<span data-ttu-id="2277f-117">双面</span><span class="sxs-lookup"><span data-stu-id="2277f-117">2</span></span>|<span data-ttu-id="2277f-118">仅当支票确认证书时, 才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="2277f-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="2277f-119">无须</span><span class="sxs-lookup"><span data-stu-id="2277f-119">require</span></span>|<span data-ttu-id="2277f-120">第三章</span><span class="sxs-lookup"><span data-stu-id="2277f-120">3</span></span>|<span data-ttu-id="2277f-121">在允许证书之前, 需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="2277f-121">Require a successful CRL check before allowing a certificate</span></span>|



