---
title: Windows 更新 API 概述
description: 适用于企业的Windows 更新部署服务为组织提供了对设备提供的更新的控制权。
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: e6bb301bac7a261db8284ad40a5914a11cca5171
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437525"
---
# <a name="windows-updates-api-overview"></a>Windows 更新 API 概述

Windows 更新企业版部署服务通过批准、计划和保护Windows 更新提供的内容来控制设备更新。

## <a name="why-use-the-windows-update-for-business-deployment-service"></a>为何使用 Windows 更新 for Business 部署服务？

IT 专业人员和管理工具供应商都可以使用部署服务执行以下操作：
* 将更新部署计划为在特定日期开始。
* 使用丰富的表达式在几天或几周内分阶段部署。
* 绕过预配置的适用于企业的 Windows 更新策略以立即部署安全更新。
* 通过针对独特设备群体量身定制的部署，确保覆盖组织中的硬件和软件。

目前，部署服务支持管理 Windows 功能更新和加快 Windows 安全更新。 若要在 Windows 更新 for Business 上下文中详细了解部署服务，请参阅[部署服务概述](/windows/deployment/update/deployment-service-overview)。

## <a name="prerequisites"></a>先决条件

若要使用部署服务，组织必须具有以下订阅之一：
* Windows 10 企业版 E3 或 E5 (包含在 Microsoft 365 F3、E3 或 E5) 
* Windows 10 教育版 A3 或 A5 (包含在 Microsoft 365 A3 或 A5) 
* Windows 虚拟桌面访问 E3 或 E5
* Microsoft 365 商业高级版

此外，部署服务管理的设备必须：
* 加入 Azure AD 或加入混合 AD
* 运行以下Windows 10版本之一：Windows 10 专业版、Windows 10 企业版、Windows 10 教育版、Windows 10 专业教育版
* 已安装Windows 10版本 1709 或更高版本

## <a name="enroll-devices-to-be-managed"></a>注册要管理的设备

若要开始使用部署服务，请 [在更新管理中注册设备](windowsupdates-enroll.md)。

## <a name="approve-and-schedule-windows-content-delivered-from-windows-update"></a>批准并计划从Windows 更新传送的 Windows 内容

部署服务简化了针对不同设备生态系统的审核、审批、计划和部署内容。 存在更新目录以提供为审批量身定制的视图，帮助你专注于重要的审批决策，并避免需要对相关更新的深度列表进行排序。

选择要部署的更新后，可以计划部署以在将来开始，或在一段时间内进行部署。 如果选择在一段时间内部署更新，则部署服务会自动优化设备的更新顺序。 如果可能，服务会对设备进行排序，以确保在部署的早期就表示硬件和软件资产的多样性，以最大程度地减少可能遇到意外更新问题的设备数。 

详细了解部署服务：
* [软件更新](windowsupdates-software-updates.md)
* [部署](windowsupdates-deployments.md)
* [安排部署](windowsupdates-schedule-deployment.md)

## <a name="immediately-deploy-an-update-when-critical-needs-arise"></a>在出现关键需求时立即部署更新

在出现严重安全问题时，可以使用部署服务绕过标准更新策略并加快安全更新的部署。

若要了解详细信息，请参阅 [部署加速的安全更新](windowsupdates-deploy-expedited-update.md)。

## <a name="protect-devices-by-default"></a>默认情况下保护设备

享受 [保护措施](/windows/deployment/update/safeguard-holds) 的优势，防止存在质量或兼容性问题的设备安装更新，否则导致故障或回滚。 对于部署Windows 11，部署服务会扩展这些保护措施，以进一步保护设备。 当设备升级到Windows 11时，Microsoft 使用机器学习算法来监视 Windows 生态系统的广度。 对于被识别为出现升级后问题风险较高的设备，部署服务会在调查和确认问题时应用早期保护措施来保护这些设备。

若要了解详细信息，请参阅 [管理部署的保障措施](windowsupdates-manage-safeguards.md)。

此外，还可以配置组织特有的监视规则。 这些规则可以根据设备信号（如回滚）发送警报或暂停部署。

若要了解详细信息，请参阅 [管理部署的监视规则](windowsupdates-manage-monitoring-rules.md)。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

请参阅 [Microsoft Graph beta 中的 Windows 更新 API](/graph/api/resources/windowsupdates-updates?view=graph-rest-beta&preserve-view=true)。
