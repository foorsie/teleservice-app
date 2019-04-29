<template>
    
    <section id="ticket-slide">
        <div class="ticket-slide-header slide-padding">
            <div class="ticket-nav">
                <div class="prev"><h3><span class="icon-container"><i class="material-icons">navigate_before</i></span>Prev</h3></div>
                <div class="next"><h3>Next<span class="icon-container"><i class="material-icons">navigate_next</i></span></h3></div>
            </div>
            <div class="ticket-details">
                <div class="ticket-no">
                    <h1>Ticket Header</h1>
                </div>
                <div class="ticket-details-small">
                    <div class="detail-title">
                        <h4>Title</h4>
                        <h4>Status</h4>
                        <h4>Created</h4>
                        <h4>last Updated</h4>
                    </div>
                    <div class="detail-value">
                        <p>Battery Guard</p>
                        <p>Reassigned</p>
                        <p>12 February 2018</p>
                        <p>22March 2018</p>
                    </div>
                </div>
                
            </div>
            
        </div>

        <div class="ticket-slide-vehicle-details slide-padding">
            <h3 class="section-title">Vehicle Details</h3>
            <div class="ticket-details-small">
                    <div class="detail-title">
                        <h4>Brand</h4>
                        <h4>Vehicle</h4>
                        <h4>Vin Number</h4>
                        <h4>Registration</h4>
                        <h4>First registration</h4>
                    </div>
                    <div class="detail-value">
                        <p>BMW</p>
                        <p>116 hatch 5Dr 1.5d ED StopStart EU6 Plus 6Spd</p>
                        <p>1JXMN1670VM6D0L</p>
                        <p>GB60SEP</p>
                        <p>21 March 2018</p>
                    </div>
                </div>
        </div>

        <hr>
    </section>


</template>


<script>
export default {
    name: 'ticketslide'
}
</script>


<style lang='scss'>
@import '../global.scss';

.detail-title, .detail-value{
            h4, p{
                margin-bottom:5px;
            }
            h4{
                text-align: right;
            }
            p{
                margin-left:10px;
            } 
        }




.ticket-nav, .ticket-details{
    display: grid;
    grid-template-columns: 1fr 1fr; 

    .ticket-details-small {
        display: grid;
        grid-template-columns: 1fr 1fr;
        padding-top: 5px;

        
    }
}

.slide-padding{
    padding:1em 2em;
}

#ticket-slide{
    width: 500px;
    position: absolute;
    right: 0;
    background: $white;
    height: 100%;
    z-index: 9999;
    box-shadow: -4px 3px 4px rgba(0, 0, 0, 0.1);

    &:before{
        font-family: "Font Awesome 5 Free";
        content: "\f00d";
        font-size: 20px;
        font-weight: 900;
        left: -30px;
        top: 10px;
        position: absolute;
    }


    .ticket-slide-header{
        background: $color-body;
        margin: 0;
        
        min-height: 160px;

        .ticket-nav{
            margin-bottom: 20px;
        }

        h1{
            @include color($color-secondary);
            @include size(24px);
            margin: 0;      
        }

        .next{
            text-align: right;
        }
    }

    // TICKET VEHICLE DETAILS

    .ticket-slide-vehicle-details{

        .section-title{
            margin: 1em 0;
        }

        .ticket-details-small{
            display: grid;
            grid-template-columns: 1fr 3fr; 
            
            h4{
                text-align: left;
            }
        }
        
    }

}




</style>
