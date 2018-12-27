changing pom.xml index.html
<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" />


add _nav.ts

changing main.component.html

adding content/assets

import { PerfectScrollbarModule } from 'ngx-perfect-scrollbar';
import { PerfectScrollbarConfigInterface } from 'ngx-perfect-scrollbar';
const DEFAULT_PERFECT_SCROLLBAR_CONFIG: PerfectScrollbarConfigInterface = {
    suppressScrollX: true
};

        AppAsideModule,
        AppBreadcrumbModule.forRoot(),
        AppFooterModule,
        AppHeaderModule,
        AppSidebarModule, 
BsDropdownModule.forRoot(),
to app.module.ts

private principal: Principal, public loginService: LoginService , public loginModalService: LoginModalService
 to constructor parameter and
isAuthenticated(): boolean {
        return this.principal.isAuthenticated();
    }
 imgSrc(brand) {
        return brand.src ? brand.src : '';
    }
    imgWidth(brand) {
        return brand.width ? brand.width : 'auto';
    }

    imgHeight(brand) {
        return brand.height ? brand.height : 'auto';
    }

    imgAlt(brand) {
        return brand.alt ? brand.alt : '';
    }
openLogin() {
        this.modalRef = this.loginModalService.open();
    }
logout() {
        this.headerPosition = 'relative';
        document.body.classList.remove('sidebar-lg-show');
        this.loginService.logout();
        this.router.navigate(['']);
    }
 public navItems = navItems;
    public sidebarMinimized = true;
    private changes: MutationObserver;
    public element: HTMLElement = document.body;
modalRef: NgbModalRef;
 headerPosition: String = 'relative';
 navbarBrandFull: any = { src: '../../content/assets/img/brand/logo.svg', width: 89, height: 25, alt: 'CoreUI Logo' };
    navbarBrandMinimized: any = "{src: 'content/assets/img/brand/sygnet.svg', width: 30, height: 30, alt: 'CoreUI Logo'}";
to main.component.ts
